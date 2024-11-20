# GymHub
This application aims to manage the information of *trainers, **trainees* and their training activities in a gym. It allows trainees to register and modify their profiles, partner with a trainer and record details of their workouts.
Each category includes time spent training and the associated trainer.

## Project Architecture
The application uses *two microservices*:

### Main microservice


###  Link application GymHub

1. *Apprentice Management:🏋🏻‍♀*
   - Register a new apprentice.
   - Modify the trainee profile (name, age, experience level, etc.).
   - Associate a trainee with a trainer.
   - Delete your profile
   - Search your data

2. *Coach Management:💪*
   - Register a coach with your basic information (name, specialization, years of experience).
   - Assign trainees to trainers.

3. *Training Record:*
   - Categorize workouts into *Upper Body💪, **Leg🦵* and *Cardio🫀*.
   - Record the time spent on each workout.
   - Assign a coach to each traini

   ## second microservice📓

   - Activities Microservice
Registration and storage of training activities. It uses a non-relational database (*MongoDB*).
#### Features:
- Save activities with specific details:
  - Learner ID.
  - Username of the trainee.
  - Trainer ID.
  - Name of the training.
  - Date and duration of the training.
  - Type of training.
- Provide activity data to the main microservice for monthly reports.

   ### Project structure
📂 GymHub
🛢backups
⚙ config
⛲Src
   ├── 📂 application
    ├── ├── 📂 domain
    ├── ── ├── 📂 abstract-classes
        ├──   ├── ├── 📂 models
            ├──   ├── ├── ├── 📂  enums
             ├──   ├── ├── ├── 📂   auth
    ├──  📂   infrastructure
    ├── ├──     📂 dto
        ├── ├── 📂 modules
        📂 routes
        📂 repositories
            📂 config
        📂 services
        




  ## Hexagonal architecture
![hexagonal architecture](C:\Users\laura\OneDrive\Imágenes\Capturas de pantalla\architecture.png)

## Technical requirements
### 1. *Programming Languages:*
- node.js
- TypeScript
- mongoDB
- MySql
- swagger

### 2. *Bookstores*
 
-   MySQL2 

	    
        npm install --save mysql2
        
	    
        npm install --save-dev @types/node
        

-   MongoDB

        
        npm install mongoose @types/mongoose
        
        
        yarn add mongoose @types/mongoose
	    

-	Express 

	    npm install express --save
	    npm install @types/express

-   Classvalidator 

	    npm i class-validator
	    npm i @types/class-validator
	
-  	Config<br>

	    npm i config
	    npm i --save-dev @types/config

- 	Nodemon

        npm install --save-dev nodemon
        npm install dotenv
        npm install --save-dev @types/dotenv

-   Swagger

        npm install swagger-ui-express swagger-jsdoc @types/swagger-ui-express @types/swagger-jsdoc


## Collaborators

    - Dayana Montoya 
    - Dilbani Enriquez 
    - German Guerrero
    - Heidy florez
    - Laura Zuluaga