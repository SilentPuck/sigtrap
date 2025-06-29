Security Policy
🧠 Why C?

This project is written in C intentionally, with full awareness of its power and risks.
🔒 Memory Safety

This tool is built and tested with:

    -Wall -Wextra -Wpedantic
    -fsanitize=address -fsanitize=undefined
    valgrind --leak-check=full
    Stack protector and hardened flags

📫 Contact

Report any issues to: silentpuck@protonmail.com