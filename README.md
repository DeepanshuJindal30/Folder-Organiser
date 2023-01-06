# Folder-Organiser

This script will move all the files in a given folder (specified by the folderpath variable) that have a file extension specified in the dic_ex dictionary into separate folders based on the type of file they are.

For example, all files with a .mp4 or .webm extension will be moved into a folder called VideoFiles. If the VideoFiles folder does not exist in the specified folderpath, it will be created before the files are moved. Similarly, all .txt and .docx files will be moved into a TextFiles folder, all .mp3 files will be moved into an AudioFiles folder, and all .png and .jpg files will be moved into an ImageFiles folder.

The file_finder function takes a folder_path and a tuple of file_ex (file extensions) as input and returns a list of all the files in the folder_path that have a file extension specified in the file_ex tuple.

The shutil.move function is used to move the files from their original location to the new folder. The os.mkdir function is used to create the new folder if it does not already exist.
