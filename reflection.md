# Reflection: AI-Assisted Buffer Overflow Visualization

**Project:** Buffer Overflow Interactive Visualizer
**Focus Area:** Stack-Frame Memory Corruption

## Experience and Deepened Understanding
Building this interactive visualization really changed how I view buffer overflows. Instead of just seeing them as an abstract security issue, I now understand the actual layout in memory. When learning about stack-based buffer overflows in class, it is easy to just memorize terms like buffers, saved frame pointers (SFP), and return addresses (RET) without grasping how they sit next to each other physically.

Creating a tool that shows these parts forced me to map out a real stack frame. Coding the logic to take text input and put it into simulated memory blocks character by character made the idea of an overflow much more real. Watching the UI turn red the exact second a string outgrows its array and starts overwriting the SFP and Return Address made it obvious how missing a simple bounds check leads to hijacked code. The project connected the dots between theoretical C code bugs and actual memory mechanics, making it clear why memory management is so important.

## AI-Assisted Workflow
To build this app, I used a back-and-forth process with AI:

1. **Setup and Layout:** I started by asking the AI to write a single HTML and JavaScript file using Tailwind CSS for a clean look. I told it I needed a mock memory stack with color-coded sections for the Buffer, SFP, and RET.
2. **Logic and Mapping:** Next, I had the AI write the JavaScript to connect a text input box to those visual blocks. I wanted to make sure that once the text got longer than the buffer, the extra characters would visibly spill over into the critical memory areas.
3. **Tweaking the UI:** After getting the base code, I reviewed it and asked for better visual cues. For example, I had the AI change the color of overwritten blocks to red and add an alert message so users know immediately when memory corruption happens.
4. **Testing:** Finally, I tested the app myself. I adjusted the buffer sizes and layout to make sure the visual flow made sense and accurately showed a classic stack smashing attack.

Using AI let me focus on the educational side of the app instead of getting stuck typing out basic UI code, which helped me finish a much cleaner teaching tool.
