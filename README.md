Introduction: 
This dataset comprises a collection of photos sourced from JiaGuWen on GitHub (https://github.com/Chinese-Traditional-Culture/JiaGuWen). It provides visual representations of ancient Chinese characters.

I gathered descriptions for the characters depicted in the photos from Hanziyuan(https://hanziyuan.net/), an online resource for exploring the origins and meanings of Chinese characters. These descriptions have been combined with the original data to create a JSON file that can be used for fine-tuning the LLAVA model.

Limitation: 
Current Problem 1: There are two types of descriptive information for these characters. One is "Decomposition Notes," which is well-structured and easy to understand but covers only about 20% of the data. The other type is "Character Decomposition," which is less structured and contains redundant information, but it is guaranteed to be complete. For example: "车--Decomposition notes: two-wheeled cart; Character decomposition: Component 車 new-char 车 (name- cart-che 车車 chē)."

My current solution:  is to combine "Decomposition Notes" with "Character Decomposition" using a hyphen ("-") to create the final description for each photo.

Further questions: 
1 What would be the Standardized Structure for the description attribute and the entire json dataset?
2 How would you recommend me to do the data cleanning? 