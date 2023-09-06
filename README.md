# Text-Corrector-Python
 This code creates a simple graphical user interface (GUI) application using Tkinter to correct spelling errors in user-inputted text. It employs the TextBlob library for spelling correction and provides a user-friendly interface with input and output fields, along with a "Check" button to initiate the correction process.

*This is the flowchart for the code.


![image](https://github.com/kaniz-codes/Text-Corrector-Python/assets/138873297/81c4161b-585e-44e9-9173-f50fbfe02e82)

*Let's drive into the code step by step with explanation.

1️⃣ 𝐒𝐭𝐞𝐩 𝟏:
![codeimage-snippet_6](https://github.com/kaniz-codes/Text-Corrector-Python/assets/138873297/ba312ed5-404e-44db-95b7-207159ed0198)
- These lines import the necessary modules for the code. TextBlob is from the textblob library, which is used for natural language processing tasks such as spelling correction, and Tk and other elements are imported from the tkinter library for building the graphical user interface (GUI).

2️⃣ 𝐒𝐭𝐞𝐩 𝟐:
![codeimage-snippet_6 (1)](https://github.com/kaniz-codes/Text-Corrector-Python/assets/138873297/c9604775-e941-48ed-b84f-1f13efe4dc29)
- This function, correct_spelling, is defined to perform the spelling correction. Here's what it does:

𝐠𝐞𝐭_𝐝𝐚𝐭𝐚= 𝐞𝐧𝐭𝐞𝐫𝟏.𝐠𝐞𝐭(): It retrieves the text entered in the enter1 Entry widget and stores it in the get_data variable.
𝐜𝐨𝐫𝐫= 𝐓𝐞𝐱𝐭𝐁𝐥𝐨𝐛(𝐠𝐞𝐭_𝐝𝐚𝐭𝐚): It creates a TextBlob object from the input text, which will be used for spelling correction.
𝐝𝐚𝐭𝐚 = 𝐜𝐨𝐫𝐫.𝐜𝐨𝐫𝐫𝐞𝐜𝐭(): It corrects the spelling of the text using the correct() method of the TextBlob object and stores the corrected text in the data variable.
𝐞𝐧𝐭𝐞𝐫𝟐.𝐝𝐞𝐥𝐞𝐭𝐞(𝟎,𝐄𝐍𝐃): It clears the text in the enter2 Entry widget.
𝐞𝐧𝐭𝐞𝐫𝟐.𝐢𝐧𝐬𝐞𝐫𝐭(𝟎,𝐝𝐚𝐭𝐚): It inserts the corrected text (data) into the enter2 Entry widget.

3️⃣ 𝐬𝐭𝐞𝐩 𝟑:
![codeimage-snippet_6 (2)](https://github.com/kaniz-codes/Text-Corrector-Python/assets/138873297/7bc8978c-427a-470b-949b-b29b10a0f857)
- This function, main_window, is defined to create the main GUI window. Here's what it does:

𝐠𝐥𝐨𝐛𝐚𝐥 𝐞𝐧𝐭𝐞𝐫𝟏, 𝐞𝐧𝐭𝐞𝐫𝟐: This line declares enter1 and enter2 as global variables, which allows them to be accessed and modified within the function.
𝐰𝐢𝐧 = 𝐓𝐤(): It creates the main Tkinter window and assigns it to the variable win.
𝐰𝐢𝐧.𝐠𝐞𝐨𝐦𝐞𝐭𝐫𝐲("𝟓𝟎𝟎𝐱𝟑𝟖𝟎"): It sets the size of the window to 500 pixels in width and 380 pixels in height.
𝐰𝐢𝐧.𝐫𝐞𝐬𝐢𝐳𝐚𝐛𝐥𝐞(𝐅𝐚𝐥𝐬𝐞, 𝐅𝐚𝐥𝐬𝐞): It disables window resizing both horizontally and vertically.
𝐰𝐢𝐧.𝐜𝐨𝐧𝐟𝐢𝐠(𝐛𝐠="𝐁𝐥𝐚𝐜𝐤"): It sets the background color of the window to black.
𝐰𝐢𝐧.𝐭𝐢𝐭𝐥𝐞("𝐊𝐚𝐧𝐢𝐳'𝐬 𝐂𝐨𝐫𝐫𝐞𝐜𝐭𝐨𝐫 𝐁𝐨𝐱"): It sets the title of the window to "Kaniz's Corrector Box."

4️⃣ 𝐬𝐭𝐞𝐩 𝟒:
![codeimage-snippet_6 (3)](https://github.com/kaniz-codes/Text-Corrector-Python/assets/138873297/55c2aa64-de1c-471d-96fb-0cd611a608bf)
- This code creates a label widget (label1) and places it in the window. Here's what it does:

𝐋𝐚𝐛𝐞𝐥(𝐰𝐢𝐧, 𝐭𝐞𝐱𝐭="𝐈𝐧𝐜𝐨𝐫𝐫𝐞𝐜𝐭 𝐒𝐩𝐞𝐥𝐥𝐢𝐧𝐠", 𝐟𝐨𝐧𝐭=("𝐓𝐢𝐦𝐞 𝐍𝐞𝐰 𝐑𝐨𝐦𝐚𝐧",𝟐𝟓,"𝐛𝐨𝐥𝐝"), 𝐛𝐠="𝐆𝐫𝐚𝐲", 𝐟𝐠="𝐖𝐡𝐢𝐭𝐞"): It creates a label with the text "Incorrect Spelling," specified font settings, and background/foreground colors.
𝐥𝐚𝐛𝐞𝐥𝟏.𝐩𝐥𝐚𝐜𝐞(𝐱=𝟏𝟎𝟎,𝐲=𝟐𝟎,𝐡𝐞𝐢𝐠𝐡𝐭=𝟓𝟎,𝐰𝐢𝐝𝐭𝐡=𝟑𝟎𝟎): It positions the label at coordinates (100, 20) within the window, sets its height to 50 pixels, and width to 300 pixels.

5️⃣ 𝐒𝐭𝐞𝐩 𝟓:
![codeimage-snippet_6 (4)](https://github.com/kaniz-codes/Text-Corrector-Python/assets/138873297/589561a2-e912-491e-a758-36d7050d1c27)
- This code creates an Entry widget (enter1) for user input and places it in the window. Here's what it does:

𝐄𝐧𝐭𝐫𝐲(𝐰𝐢𝐧, 𝐟𝐨𝐧𝐭=("𝐓𝐢𝐦𝐞 𝐍𝐞𝐰 𝐑𝐨𝐦𝐚𝐧",𝟐𝟓)): It creates an Entry widget with a specified font.
𝐞𝐧𝐭𝐞𝐫𝟏.𝐩𝐥𝐚𝐜𝐞(𝐱=𝟓𝟎, 𝐲=𝟖𝟎, 𝐡𝐞𝐢𝐠𝐡𝐭=𝟓𝟎, 𝐰𝐢𝐝𝐭𝐡=𝟒𝟎𝟎): It positions the Entry widget at coordinates (50, 80) within the window, sets its height to 50 pixels, and width to 400 pixels.

6️⃣ 𝐒𝐭𝐞𝐩 𝟔:
![codeimage-snippet_6 (5)](https://github.com/kaniz-codes/Text-Corrector-Python/assets/138873297/938a1daa-46f0-459e-b132-138bc96c5d11)
- This code creates another label widget (label2) for displaying corrected text and places it in the window. It's similar to the label1 creation and placement.

7️⃣ 𝐒𝐭𝐞𝐩 𝟕:
![codeimage-snippet_6 (6)](https://github.com/kaniz-codes/Text-Corrector-Python/assets/138873297/df790b28-1b4c-4825-9ab2-336bf4e66525)
- This code creates another Entry widget (enter2) for displaying the corrected text and places it in the window. It's similar to the enter1 creation and placement.

8️⃣ 𝐒𝐭𝐞𝐩 𝟖:
![codeimage-snippet_6 (6)](https://github.com/kaniz-codes/Text-Corrector-Python/assets/138873297/f534e296-9db8-4e01-af65-7308f8abba29)
- 
