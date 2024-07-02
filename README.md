# Drakkar
Web app using HTML, CSS, JavaScript, PHP, and Bash for interactive learning and scripting. Requires PHP server or Docker for deployment.

My HTML App

A web application powered by HTML, CSS, JavaScript, PHP, and Bash commands. Explore and learn web development and command-line scripting with this interactive app.

Key Features:
- Responsive HTML/CSS frontend with interactive elements.
- Server-side processing using PHP.
- Integration of Bash scripts for automating tasks.
- Requires PHP built-in server or can be deployed using Docker.


### Work-in-Progress (WIP) Status
This application is currently a work-in-progress (WIP) source. While the core functionalities are in place and it is almost ready to work perfectly, please note the following:
- **Creating a Tutorial**: We are lost here https://docs.google.com/document/d/1M9W6reA7zW5WYmkLBI8DwFDExwce8JQFuZK3ixiNICQ/edit?usp=sharing
- **Cleaning of Unnecessary Files**: The application may contain unnecessary files (garbage) that need to be cleaned up.
- **Testing Status**: While important aspects of development have been tested, the testing coverage is not yet exhaustive.

### Target Audience:

Developers and learners interested in web development and command-line scripting. Anyone interested in food and nutrients, and in creating recipes with a database granted and supported by government agents (Read the Disclaimer).

### Future Development
We are continuously working to improve the application by refining features, enhancing performance, and expanding test coverage. Your feedback and contributions are welcome as we strive to make this application even better.

Feel free to clone, explore, and contribute to this project!


## Instructions

1. * Pull the Docker Image:
   sudo docker pull perevictor/alpinedrakkar-php-bash_commands0
    This is 39.77 MB, but you can also use perevictor/alpinedrakkar-php-mariadb-bash_commands0 107.29 MB instead
2. * Run the container:
   sudo docker run -d --name drakkar0 perevictor/alpinedrakkar-php-bash_commands0
3. * Copy to your host the tar and read the original Dockerfile and Tutorial: 
   sudo docker cp drakkar0:/etc/Dockerfile.tar.gz .
4. * To get started, clone the repository and follow the setup instructions to run the app locally. After cloning the 'Drakkar' repository or downloading the tar.gz (https://github.com/pere000/Drakkar/tree/main), decompress the drakkarOceans.tar.gz file to obtain the 'www' folder. Place this folder in your desired location to run the application, and navigate to it using your command line interface.

Inside the 'www' folder, execute the necessary commands to ensure your server (whether using PHP built-in or the Docker image) recognizes and hosts the application's folders and files.
  
		~ Docker users: sudo docker run --name runtest1 -dp 8080:80 -v "$(pwd)":/var/www perevictor/alpinedrakkar-php-bash_commands0

		~ PHP built-in users: php -S localhost:8080 .
     
Access the domain through http://localhost:8080/index.html


# Disclaimer:

## Nutrient Data Attribution
The nutrient data main table used in this application is sourced from the 'Norwegian Directorate of Health of the University of Oslo' and the 'Norwegian Food Safety Authority' under the MIT License. We attribute and comply with their licensing terms by providing appropriate copyright notices.

## User-generated Content
Users of this application have the ability to create and modify nutrient values, including generating "fake recipes" based on this data. However, it is important to note that this application does not grant the right to publicly distribute or publish prescriptions based on real-world data from the aforementioned licensing agents.
