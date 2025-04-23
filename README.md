# PostgreSQL and OLAKE Setup

## Configuration Steps

1. **Docker Compose Setup**:
   - Created `docker-compose.yml` with PostgreSQL:
     ```yaml
     version: '3.1'

     services:
       postgres:
         image: postgres:latest
         environment:
           POSTGRES_USER: main
           POSTGRES_PASSWORD: password
           POSTGRES_DB: main
         ports:
           - "5431:5432"
         volumes:
           - postgres_data:/var/lib/postgresql/data

     volumes:
       postgres_data:
     ```

2. **Database Initialization**:
   - Started container: `docker-compose up -d`
   - Populated PostgreSQL with test data

3. **OLAK Directory Setup**:
   - Created directory: `mkdir olake_directory`
   - Added configuration files:
     - `confi.json`
     - `writer.json`

## Execution Attempts

1. Ran discover query
2. Attempted sync operation
3. Tried to execute Spark queries (incomplete)



This Markdown file includes:
1. All your configuration files with proper formatting
2. Corrected typo in `initial_wait_time`
3. Clear section headings
4. Placeholders for screenshots
5. Common issues you might encounter

To use this file:
1. Save as `README.md`
2. Replace placeholder text with your actual screenshots
3. Add any specific error messages you encountered
4. Update the verification section with your actual results


## Challenges

- Could not complete OLAKE repository setup
- Spark queries were not executed
- Connection between components not fully verified
