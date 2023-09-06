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

