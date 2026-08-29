<div align="center" width="50">

<img src="https://user-images.githubusercontent.com/74038190/213760705-0d5bf320-4f43-4352-b74b-0889ae726bf7.gif" href="https://github.com/abdelrahmadahmedelshahat-oss" alt="Hello Coders" width="60%"/> <br>
<img src="https://user-images.githubusercontent.com/74038190/221352989-518609ab-b4d1-459e-929f-a08cd2bd9b3c.gif" href="https://github.com/abdelrahmadahmedelshahat-oss" alt="Cybersecurity" width="40%"/><br>

# Hi, I'm Abdelrahman Ahmed Elshahat 👋

**Cybersecurity Learner | C++ & Data Structures | Linux Enthusiast**

<details>
<p><strong> <summary> Currently learning & building : </summary> </strong></p>

🔐 On my way to becoming a Cybersecurity Analyst — building the fundamentals first, the right way.

</details>

![Totals Hits](https://komarev.com/ghpvc/?username=abdelrahmadahmedelshahat-oss&style=flat&color=orange&label=PROFILE+VIEWS)
![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fabdelrahmadahmedelshahat-oss&count_bg=%2379C83D&title_bg=%23555555&icon=mediafire.svg&icon_color=%23E7E7E7&title=HITS&edge_flat=false)
[![telegram badge](https://img.shields.io/badge/Contact-Telegram-grey?style=flat&logo=telegram)](https://t.me/abdelrahmadahmedelshahat)

</div>

<hr></hr>

![tools_I_use](https://img.shields.io/badge/-%F0%9F%9A%80%20Tools%20I%20use-orange)
![semicolon](https://img.shields.io/badge/-%3A-orange)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=c%2B%2B&logoColor=white)
![OOP](https://img.shields.io/badge/OOP-3776AB?style=flat&logo=cplusplus&logoColor=white)
![Data Structures](https://img.shields.io/badge/Data_Structures-FF6F00?style=flat&logo=unrealengine&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/GNU%20Bash-4EAA25?style=flat&logo=GNU%20Bash&logoColor=white)
![Git](https://img.shields.io/badge/GIT-E44C30?style=flat&logo=git&logoColor=white)
![Vscode](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=flat&logo=visual%20studio%20code&logoColor=white)
![TryHackMe](https://img.shields.io/badge/TryHackMe-212C42?style=flat&logo=tryhackme&logoColor=red)

```cpp
// about_me.cpp

#include <iostream>
#include <vector>
#include <string>

class Me {
private:
    std::string name = "Abdelrahman Ahmed Elshahat";
    std::vector<std::string> currentSkills = {
        "C++", "OOP", "Data Structures", "Linux Basics"
    };
    std::vector<std::string> learningPath = {
        "Networking", "Linux (Advanced)", "SQL Basics",
        "Cybersecurity Fundamentals", "TryHackMe"
    };
    std::string goal = "Cybersecurity Analyst";

public:
    void introduce() {
        std::cout << "Hi, I'm " << name << std::endl;
        std::cout << "Currently mastering the fundamentals," << std::endl;
        std::cout << "one Data Structure at a time." << std::endl;
        std::cout << "Goal: " << goal << " 🔐" << std::endl;
    }
};

int main() {
    Me abdelrahman;
    abdelrahman.introduce();
    return 0;
}
