# Death counter/recognizer for Soulslike Games
This small Python script updates a text file every time a death in Dark Souls: Remaster. This works by 
taking a screenshot every set amount of time (1 second), then processing the image by applying a red channel filter 
and finally using Tesseract to recognize letters in the image, in this case we want to recognize the red text **YOU DIED** which appears 
after dying in the game.

## Compatible games:

- Dark Souls
- Dark Souls: Remastered
- Dark Souls 2
- Dark Souls 3
- Bloodborne
- Elden Ring

**Note:** You'll need to adjust the screenshot region depending on the game and resolution of your monitor.
<br> I will add game/resolution profiles in the future to make this step easier.

## Dependencies:

- [numpy](https://pypi.org/project/numpy/)
- [opencv-contrib-python](https://pypi.org/project/opencv-contrib-python/)
- [pytesseract](https://pypi.org/project/pytesseract/) (python wrapper for Tesseract binary)
- [tesseract](https://github.com/UB-Mannheim/tesseract/wiki) (Tesseract binary)

## Steps:

1) Clone repo.
2) Install dependencies.
3) Configure fileName and tesseractBinaryLocation variables accordingly.
4) Run script 