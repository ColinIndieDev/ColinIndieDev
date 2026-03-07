## Hi, I am Colin 👋

I am currently still in school (+ trying to study CS early on a university like a friend of mine by applying to it).
I like low level programming, so I used C++ and now C for graphics programming, data structures from scratch, neural networks and more!
Here, I will share my progress and code, feel free to have a peek at what I do (with my free time obviously)!

My goal is to make my OpenGL library for gamedev fully from C++ to C + the Minecraft Clone I made with C++ earlier.
Also I am trying to build my own std library from scratch with C too and with all that making cool projects f.e. games!
Now I firstly need to get very good and mastering the C programming language by using NeoVim on Arch Linux Hyprland (btw).

I also share my progress on YouTube, rarely but sometimes on itch.io if I made a game which can be played on web (with Emscripten).

```c
#include <stdlib.h>

typedef struct {
    char *usr_name;
    int age;
    char **skills;
    char **biggest_projects;
} colin_dev;

// TODO add more

int main() {
    char **skills = (char **)malloc(2 * sizeof(char *)));

    skills[0] = "C++";
    skills[1] = "C";

    char **biggest_projects = (char **)malloc(3 * sizeof(char *)));

    biggest_projects[0] = "CPL";
    biggest_projects[1] = "CPAI";
    biggest_projects[2] = "CPSTD";

    colin_dev colin = {
        .usr_name = "ColinIndieDev",
        .age = 17,
        .skills = skills,
        .biggest_projects = biggest_projects
    }

    bool vacation = false;
    bool free_time = true;
    int time = 70;
    bool fun = true;

    while (time > 0 && fun && (free_time || vacation)) {
        do_opengl();
        do_tui();
        do_stuff_from_scratch();
        do_neural_network();

        time--;
    }
    return 0;
}
```
