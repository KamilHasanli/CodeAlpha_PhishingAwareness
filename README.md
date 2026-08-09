# Phishing Awareness Training

Task 2 of my CodeAlpha Cyber Security internship. The brief was to build a presentation or short training module that teaches people how to recognize phishing emails, fake websites, and the social engineering tricks behind them.

I kept it to 10 slides on purpose — long security training decks tend to get skimmed, not read. Each slide covers one idea.

## What's in it

- What phishing actually is, and why it works on smart people too
- The main attack types: email phishing, spear phishing, whaling, smishing, vishing, clone phishing
- Five things that give away a phishing email almost every time
- How to check if a website is fake before you type anything into it
- The psychological tricks behind social engineering (urgency, authority, fear, etc.)
- A real case: the $100M+ invoice scam that hit Google and Facebook between 2013–2015
- A short list of habits that actually stop most phishing attempts
- A 3-question quiz at the end to recap

## Files

- `Phishing_Awareness_Training.pptx` — the deck
- `screenshots/` — every slide as an image, in case you don't want to open PowerPoint just to look at it

## How I made it

I didn't build this slide by slide in PowerPoint. I wrote a script (Node.js + pptxgenjs) that generates the whole deck — text, cards, icons, layout, all of it defined in code. It's slower to set up than clicking around in the PowerPoint UI, but way easier to keep everything consistent across 10 slides, and I can regenerate the whole thing in seconds if I want to change a color or fix a typo.

The icons come from the Feather icon set (react-icons), rendered to PNG, and the background gradients were generated the same way. A couple of the illustrative images I swapped in by hand afterward, in LibreOffice Impress, once I had the layout the way I wanted it.

Nothing fancy — mostly JS to generate the deck and LibreOffice to check/export the final file.
