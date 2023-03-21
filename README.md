# Visual_Cryptography_forKN_sharing

•	Important Libraries necessary for running the code:
o	Numpy
o	Pillow
o	Random
o	Open CV
o	Tqdm
o	Cryptodome
o	Os
o	Sys
o	Base64
Step1:
o	Import the Necessay packages mentioned above along with the file/image/message that needs to be shared and its size is extracted and the depending on functions are initialized (Cell 1,2 and 3 of Jupyter notebook) 
Step2:
o	Set the value of k and n ( in this case 5 and 6) .
o	 And run the NSharing Function which generated shares and stores them in the folder named, Shares.
The Next 3 parts of Step 3 are Encrypt and Decrypt using AES, DES, and Triple DES and any one can be run.
Step3a:
o	The next cell First sets the values of key and iv then it fetches the shares generated in the previous step and encrypts using AES CFB it and saves the encrypted shares in “Save_AES_enc” folder.
o	This is followed by  decryption of the shares which were generated using the same key and iv and are stored in folder “Save_AES_dec”.
Step3b: 
o	The next step is similar to the Step3a but in this we use DES instead of AEs. Just run the first cell to encrypt the shares using DES and save those in folder “Save_DES_enc”.
o	The cell following this will decrypt the shares from “Save_DES_enc” and save the images in “Save_DES_dec”
Step 3c:
o	This is similar the previous two steps but in this we use DES OFB instead of AES. Just run the first cell to encrypt the shares using DES and save those in folder “Save_TDES_enc”.
o	The cell following this will decrypt the shares from “Save_TDES_enc” and save the images in “Save_TDES_dec”
Step4:
o	The next 9 cells are divided into sub section of 3. Each set of cells do the same task of taking images from the Decrypted shares and then Merging them together to from the original image which is stored in “Deshare_AES”, “Deshare_DES” and “Dshare_TDES” depending on the section use.
NOTE: Change Directories as needed

