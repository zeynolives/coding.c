#include <iostream>
#include <string>

class Character {
protected:
    std::string profession;
    int age;
public:
    Character(std::string profession = "unemployed", int age = 16) {
        this->profession = profession;
        this->age = age;
    }
    virtual void walk() {
        std::cout << "ı can walk.\n";
    }
    virtual void talk() {
        std::cout << "ı can talk.\n";
    }
    virtual void display() {
        std::cout << "My Profession: " << profession << std::endl;
        std::cout << "My age is: " << age << std::endl;
    }
};

class MathTeacher : public Character {
public:
    MathTeacher(int age = 16) : Character("maths teacher", age) {}
    void teachmath() {
        std::cout << "I can teach maths.\n";
    }
};

class Footballer : public Character {
public:
    Footballer(int age = 16) : Character("footballer", age) {}
    void playfoot() {
        std::cout << "ı can play football\n";
    }
};

class Businessman : public Character {
public:
    Businessman(int age = 16) : Character("businessman", age) {}
    void dobusiness() {
        std::cout << "ı can do business\n";
    }
};

int main() {
    MathTeacher math_teacher(30);
    math_teacher.display();
    math_teacher.walk();
    math_teacher.talk();
    math_teacher.teachmath();

    std::cout << std::endl;

    Footballer footballer(25);
    footballer.display();
    footballer.walk();
    footballer.talk();
    footballer.playfoot();

    std::cout << std::endl;

    Businessman businessman(40);
    businessman.display();
    businessman.walk();
    businessman.talk();
    businessman.dobusiness();

    return 0;
}

