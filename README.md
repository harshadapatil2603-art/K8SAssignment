1. Created EC2 instance -k8s-ec2
<img width="700" height="400" alt="Image" src="https://github.com/user-attachments/assets/2f82330e-ecab-462f-84a7-bd83f7222283" />

2. Installed docker. kubectl and minikube on the instance.
<img width="700" height="400" alt="Image" src="https://github.com/user-attachments/assets/954118dd-e92f-444a-bdf6-bc59fc419ac3" />

3. Builded docker images for frontend and backend.
   docker build -t flask-backend:latest .
   docker build -t express-frontend:latest .

   <img width="700" height="400" alt="Image" src="https://github.com/user-attachments/assets/6f7acc92-5123-455d-b93b-44e09cf3c41c" />

4.Deployed flask application 
 kubectl apply -f kubernetes/
 kubectl port-forward service/express-frontend 3000:3000 --address 0.0.0.0
 <img width="700" height="400" alt="Image" src="https://github.com/user-attachments/assets/fa4b233b-2d99-4d29-b967-912e07fd1b96" />
 <img width="700" height="400" alt="Image" src="https://github.com/user-attachments/assets/ba53d310-6488-48b0-9b33-5b6b00913bca" />

   

5. Accessed application on below url
http://54.174.203.227:3000/

<img width="700" height="400" alt="Image" src="https://github.com/user-attachments/assets/ff198602-3fdd-4050-9a9d-54f697de3aa4" />

<img width="700" height="400" alt="Image" src="https://github.com/user-attachments/assets/c9ab3997-e0ce-4373-9392-744112201efa" />

