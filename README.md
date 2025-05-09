# Portfolio
#include <iostream>
#include <string>

using namespace std;

void showAboutMe() {
    cout << "\n--- About Me ---" << endl;
    cout << "Name: Pranjal Saket" << endl;
    cout << "Profession: Aspiring Software Developer" << endl;
    cout << "Skills: C++, Python, HTML, CSS, JavaScript" << endl;
}

void showProjects() {
    cout << "\n--- Projects ---" << endl;
    cout << "1. Calculator App (C++)" << endl;
    cout << "2. Portfolio Website (HTML/CSS/JS)" << endl;
    cout << "3. To-Do List CLI (Python)" << endl;
}

void showContact() {
    cout << "\n--- Contact ---" << endl;
    cout << "Email: john.doe@example.com" << endl;
    cout << "LinkedIn: linkedin.com/in/johndoe" << endl;
    cout << "GitHub: github.com/johndoe" << endl;
}

int main() {
    int choice;

    while (true) {
        cout << "\n=== My Portfolio ===" << endl;
        cout << "1. About Me" << endl;
        cout << "2. Projects" << endl;
        cout << "3. Contact" << endl;
        cout << "4. Exit" << endl;
        cout << "Enter your choice (1-4): ";
        cin >> choice;

        switch (choice) {
            case 1:
                showAboutMe();
                break;
            case 2:
                showProjects();
                break;
            case 3:
                showContact();
                break;
            case 4:
                cout << "Exiting portfolio. Goodbye!" << endl;
                return 0;
            default:
                cout << "Invalid choice. Please try again." << endl;
        }
    }

    return 0;
}
