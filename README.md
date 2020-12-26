# ocr
machine to transfer photo to text

from PIL import Image
import pytesseract

pytesseract.pytesseract.tesseract_cmd =  r"./Desktop/屁迪/py_project/.venv/lib/python3.9/site-packages"
img = Image.open(r'test1.png')
text = pytesseract.image_to_string(img, lang='eng')
print(text)

###permissionError: [WinError 5] 存取被拒
