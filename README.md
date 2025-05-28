# Photo Folder to PDF Converter

Batch script to convert all .jpg and .png images in a folder into a single PDF file named by a chapter number.

## Script name

Suggested script filename:  
`convert_photos_to_pdf.bat`

## How it works

- Prompts user to enter a chapter number  
- Uses ImageMagick's `magick convert` to combine all .jpg and .png files in the current folder into one PDF named `<chapter>.pdf`  
- Output PDF is created with 300 DPI resolution

## Requirements

- Windows OS  
- ImageMagick installed and added to system PATH  
- During installation, enable "Install legacy utilities (convert)" and "Add application directory to your system path"

## Usage

- Put `convert_photos_to_pdf.bat` in the folder with your images  
- Run the script (double-click or via command prompt)  
- Enter chapter number when prompted  
- Wait for PDF creation. File `<chapter>.pdf` will appear in the folder  
- Press any key to exit

## Notes

- Only .jpg and .png files are processed  
- Make sure `magick` command works in your command line (`magick -version`)  
- You can change output DPI by editing the `-density` value in the script
