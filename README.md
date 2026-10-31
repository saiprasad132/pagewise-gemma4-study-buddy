# Pagewise

**Make any page make sense.** Pagewise is a visual study buddy built for the Hacktoberfest Hack Day Gemma 4 challenge. Add an image or a PDF study document and ask Gemma 4 to explain a topic at your level or make a short quiz from it.

## Run it

1. Get a Gemini API key from [Google AI Studio](https://aistudio.google.com/app/apikey).
2. Open a terminal in this folder and run `node server.js` (Node.js required).
3. Open [http://127.0.0.1:8000](http://127.0.0.1:8000) in a browser.
4. Add an image or PDF (up to 14 MB), paste your API key, choose **Understand it** or **Quiz me**, and select **Make this click**.

The app calls `gemma-4-26b-a4b-it` through the Gemini API. The key is entered at runtime and kept in the page only; it is not stored by Pagewise. Requests go directly from the browser to Google. Avoid using a personal key on a public or shared computer.

## What it demonstrates

- **Multimodal:** sends an image or PDF document and a task prompt together to Gemma 4.
- **Focused AI tool:** explains study materials or creates a practice quiz at the learner's selected level.
- **Rapid prototype:** runs as a small static web app with no build step or server-side key storage.

## Demo flow

1. Upload a clear photo or PDF page containing a diagram or notes.
2. Select **Understand it** and ask about a specific confusing detail.
3. Generate the explanation, then switch to **Quiz me** and create a practice set.

The model is instructed to stay grounded in the visible page and flag unclear text. Review generated answers against the original material.
