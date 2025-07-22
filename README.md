# CV-Python-at-Tuwaiq
this is my work during CV python course 
from PIL import Image

# Open the image
img = Image.open('oscar.jpg')

# Resize the image
resized_img = img.resize((200, 200))

# Convert the resized image to grayscale (black & white)
converted_img = resized_img.convert("L")

# Show the converted image
converted_img.show()

# Save the converted image with a new name
converted_img.save('oscar_resized_gray.jpg')



  from PIL import Image, ImageDraw, ImageFont

# Open your image
img = Image.open('oscar.jpg')

# Create drawing context
draw = ImageDraw.Draw(img)

# Optional: Load a custom font (comment this out if you want default font)
# font = ImageFont.truetype("arial.ttf", 40)

# Draw text on the image at position (x=50, y=50)
draw.text((50, 50), "Most Famous Selfie", fill="white")  # You can change color

# Show the image
img.show()

# Save the edited image
img.save('oscar_with_text.jpg')

