Install requirements

```bash
    npm install
```

Start API:

```bash
  npm start
```

API:
1. Login
    ```
        Method: POST
        http://localhost:3000/login
   
        payload: {
          "username": "admin",
          "password": "admin"
        }
   
        Return:
        {
           "message": "Login successful",
           "token": "{token_key}"
        }
        
    ```
   
2. Get All
    ```
   Method: GET
   
   URI: http://localhost:3000/Generator
   headers: 
          key: Authorization 
          value: Bear {token_key}
   
   ```

4. Filter


    ```
      Method: GET
      
      headers: 
          key: Authorization 
          value: Bear {token_key}
   
      URI: 
        - http://localhost:3000/Generator?SKU=MF1_1
        - http://localhost:3000/Generator?id=1
     
   ```