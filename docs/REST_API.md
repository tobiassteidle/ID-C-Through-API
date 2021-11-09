**ID C Through REST API Documentation**
----

* **URL**

  /api/v1/identification


* **Method:**

  `POST`

  
* **HTTP-Headers:**
  
    `X-Rapidapi-Host`: `id-c-through.p.rapidapi.com`  
    `X-Rapidapi-Key`: `<your api key>`

  
* **Payload (Body) JSON Format**  
    ``` 
    {
        "base64": "string"
    }
    ```
  
    **base64**: Base64 encoded byte array of a document as image of pdf.    
    *Supported types:*
    - application/pdf
    - image/jpeg
    - image/png
    - image/tiff
    - *other image types possible but not tested*
    

* **Success Response:**

    * **Code:** 200 <br />
      **Content:**  
  ```    
    {
        "result": [
            {
            "page": "integer"
            "country": "string",
            "side": "enum",
            "type": "enum"
            }
        ],
        "status": "enum"
    }
    ```
  **result**: Array of id cards or passports found on document.  
  **page**: Page number on which the id cards or passports was found (for multipage PDF).  
  **country**: Name of the country from which the ID card was recognized.  
  **side**: Enum FRONT or BACK  
  **type**: Enum IDCARD, PASSPORT or RESIDENCE_PERMIT  
  **status**: Enum SUCCESS or ERROR


* **Error Response:**

    * **Code:** 415 UNSUPPORTED MEDIA TYPE
      <br />
      **Content:**
  ```
  {
    "message": "<error message>",
    "status": "ERROR"
  }
  ```

  OR

  * **Code:** 400 BAD REQUEST
    <br />
    **Content:**
    ```
    {
      "message": "<error message>",
      "status": "ERROR"
    }
    ```

  OR

    * **Code:** 404 NOT FOUND
      <br />
      **Content:**
      ```
      {
        "message": "No ID Cards or Passports detected.",
        "status": "ERROR"
      }
      ```

  OR

    * **Code:** 500 INTERNAL SERVER ERROR
      <br />
      **Content:**
      ```
      {
        "message": "<error message>",
        "status": "ERROR"
      }
      ```
