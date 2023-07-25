# Description

This project is a Face Recognition Based Attendance System implemented using Python and OpenCV. The system allows users to register new students by capturing their images and saving them along with their details such as ID and name. The system also provides a feature to change the admin password for security.

## The main features of the system include:

- New Student Registration: Users can register new students by entering their ID and name, and then capturing their images using the webcam.

- Face Recognition: Once the students are registered, the system uses the LBPH (Local Binary Patterns Histogram) face recognition algorithm to recognize the registered students from live webcam feed.

- Attendance Tracking: The system captures the student's attendance by matching their faces with the registered ones. If a student is recognized, their attendance is marked with the current date and time.

- Admin Password Protection: The system provides password protection for the admin. Only authorized users can access the system functionalities, and the admin can change the password as needed.

# How to Use

- Run the Python script to launch the application.
- To register new students, enter their ID and name, and click on "Take Images" to capture their images. Then click on "Save Profile" to save the student's information.
- To mark attendance, click on "Take Attendance" to activate the webcam and start recognition.
- The recognized students' details will be displayed in the table on the right side of the window.
- The admin can change the password by clicking on the "Change Password" option in the Help menu.

# Dependencies

    Python 3.x
    OpenCV
    Tkinter (GUI library)
    Pandas
    Numpy
    Pillow (PIL)

# How it Works

The system uses the haarcascade_frontalface_default.xml file for face detection. When registering new students, the system captures their images using the webcam and saves them in the "TrainingImage" folder. The student's details are then stored in the "StudentDetails.csv" file.

During attendance tracking, the system loads the pre-trained model from "Trainner.yml" and recognizes the faces from the live webcam feed. If a recognized student is not already marked present, their attendance is recorded in the "Attendance_List.csv" file, and their details are displayed in the table on the GUI.

The attendance data can be saved to a CSV file by clicking on the "Quit" button, or it will be automatically saved after every 10 seconds.

## Authors

    Umang Laad - https://github.com/UmangLaad
    Viral Parikh - https://github.com/Viral1006
    Gautam Sharma - https://github.com/developergautam07

### Credits

This project is inspired by various tutorials and resources available on face recognition and OpenCV. Special thanks to the OpenCV community for providing valuable documentation and tutorials.
