## Project Overview
This is a simple Java "Hello World" application built using **Maven** and integrated with **Jenkins** for CI/CD.  
The project demonstrates a basic build pipeline, from code checkout to artifact creation, as a first step into continuous integration.

## Features
- Java application printing "Hello, Jenkins + Maven!"
- Maven build with `clean package` goal
- Jenkins Freestyle and Pipeline compatible
- Demonstrates basic CI/CD workflow

## Prerequisites
- Jenkins 
- Java JDK 8 or 11
- Maven
- Git 

Project Structure

<img width="282" height="270" alt="image" src="https://github.com/user-attachments/assets/c63d7db4-b83c-494b-bd83-a7bcbb086492" />


## Jenkins Freestyle Job Build Steps

1. **Create Freestyle Job**  
   - Go to **Jenkins → New Item → Freestyle project → Enter Name → OK**

2. **Link GitHub Repository**  
   - Scroll to **Source Code Management → Git**  
   - Enter **Repository URL**:  
     ```
     https://github.com/vamshireddy903/Task-8.git
     ```  
   - Add credentials if the repo is private  
   - Select branch to build (e.g., `main`)

3. **Configure Build Step**  
   - Scroll to **Build → Add build step → Invoke top-level Maven targets**  
   - Select **Maven Version** (configured in Jenkins)  
   - Set **Goals**:  
     ```
     clean package
     ```

4. **Save & Build**  
   - Click **Save → Build Now**  
   - Check **Console Output** → Should show:  
     ```
     [INFO] BUILD SUCCESS
     ```

---

<img width="1906" height="1001" alt="image" src="https://github.com/user-attachments/assets/bc2df93f-4e1c-4b6f-925d-eff6f27d9b3a" />

<img width="1881" height="937" alt="image" src="https://github.com/user-attachments/assets/84889a56-2f91-4d95-97f0-ac7144e1a9ca" />

<img width="1906" height="871" alt="image" src="https://github.com/user-attachments/assets/90607d39-2724-4375-bf5f-48c3938d41c5" />



