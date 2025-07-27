# Work Athlete Dashboard

The **Work Athlete Dashboard** is a lightweight, static productivity tracker designed for rapid 30-minute work sprints (sets) combined with micro-workouts. It functions as a daily dashboard where each "set" includes:
- A **goal/intention field** (set your focus for the sprint).
- A **timer** that counts up from 00:00 to a max of 30:00.
- **Checkboxes** for marking work and movement completion.
- A **notes field** for documenting what was accomplished.
- **Export to PDF** functionality to archive daily sets.

---

## Features

- **Local Persistence:**  
  Data for each day is saved in `localStorage` and automatically resets when a new day begins.

- **Add Unlimited Sets:**  
  Start with one set and add as many as you need. Each set tracks elapsed time individually.

- **Export to PDF:**  
  All sets and notes for the day are exported into a clean PDF file with a single click.

- **Elapsed Time Tracking:**  
  Each set’s timer records the actual time spent on a task (up to 30 minutes), allowing historical analysis of task durations.

- **Simple UI:**  
  Designed with a light mode aesthetic for clarity and focus.

---

## Future Enhancements

The following ideas are **planned for future development** but are not implemented in the current MVP:

### **1. Speech-to-Text for Notes**
- Add a **record button** for each set that enables voice dictation.
- Convert recorded audio into text using a local **speech-to-text engine** (e.g., [OpenAI Whisper](https://github.com/openai/whisper) or [Vosk](https://alphacephei.com/vosk/)).

### **2. LLM-Based Summarization**
- After recording voice notes, automatically pass the raw text through a **local LLM** (such as LLaMA or GPT4All).
- Generate a **clean summary** of the task for that set.
- Optionally add **bullet points or formatted takeaways** for clarity.

### **3. Daily Summary**
- When exporting the PDF, generate a **daily meta-summary** (e.g., "You completed 6 sets totaling 2h 50m of work. Focus areas: Design, Code, Research...").

### **4. Audio Notes**
- Save **raw audio files** locally (or in-browser memory) for playback and future transcription.

---

## Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/YOUR-USERNAME/work-athlete-dashboard.git
   cd work-athlete-dashboard
