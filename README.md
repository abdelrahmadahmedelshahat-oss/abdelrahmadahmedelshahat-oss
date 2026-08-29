<div align="center">

<!-- Cybersecurity / Hacker GIF -->
<img
  src="YOUR_CYBERSECURITY_HACKER_GIF_URL"
  alt="Cybersecurity Hacker"
  width="65%"
/>

<br>

<!-- Personal Cybersecurity Banner -->
<img
  src="YOUR_PERSONAL_CYBERSECURITY_IMAGE_URL"
  alt="Abdelrahman - Cybersecurity Journey"
  width="45%"
/>

<br>

# Hi, I'm Abdelrahman Ahmed Elshahat 👋

### 🔐 Cybersecurity Learner | C++ Developer | Linux Enthusiast

<p>
  Building my foundation in programming, Linux, networking and cybersecurity.
  <br>
  Learning step by step and turning what I learn into practical projects.
</p>

</div>

---

## 🧑‍💻 About Me

```cpp
// about_me.cpp

#include <iostream>
#include <vector>
#include <string>

class Me {
private:

    std::string name = "Abdelrahman Ahmed Elshahat";

    std::vector<std::string> skills = {
        "C++",
        "OOP",
        "Data Structures",
        "Linux Basics",
        "Git & GitHub"
    };

    std::vector<std::string> currentlyLearning = {
        "Networking",
        "Linux",
        "Cybersecurity Fundamentals",
        "Bash",
        "SQL",
        "TryHackMe"
    };

    std::string goal =
        "Build a strong foundation in Cybersecurity";

public:

    void introduce() {

        std::cout
            << "Hi, I'm " << name << "\n\n";

        std::cout
            << "I'm building my technical foundation "
            << "through C++, Linux and Cybersecurity.\n";

        std::cout
            << "I believe in learning the fundamentals "
            << "before moving to advanced topics.\n";

        std::cout
            << "Goal: " << goal << " 🔐\n";
    }
};

int main() {

    Me abdelrahman;

    abdelrahman.introduce();

    return 0;
}
