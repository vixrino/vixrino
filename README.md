- MSc student in AI
- Interested in 3D deep learning, transformers, GPU computing 

[Resume](https://drive.google.com/file/d/19SQQZMWSpm4dyWVv0-J0erS0qMxDHGaV/view?usp=sharing)


---

![](https://komarev.com/ghpvc/?username=vixrino&color=blueviolet&style=flat)



$body = @{ 
  project_id = 4 
  schema_id = 2 
  name = "CERFA surendettement" 
  ocr_provider = "MISTRAL" 
  required_operators = 2 
  expected_page_count = 12 
} | ConvertTo-Json 
 
Invoke-RestMethod "http://localhost:8001/api/v1/datasets" -Method Post -ContentType  
"application/json" -Body $body 
