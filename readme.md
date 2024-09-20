
# Task-1
step by step guide to access the encrypted file. Lets get started:

1. Download the file named as test.txt (This file contains the encrypted message which is coverted to 32 bits hex code).

2. Download the `symmetric.key` file, this file contains the key to decrypt the encrypted file.

After downloading both the files, follow the steps to decrypt the file.

1. Open the terminal.

2. Please go to the directory where both the downloaded files are. Lets say, we have both the files in `Downloads` folder and we are currently in the root folder. Then, we can use this command to go to that respective folder.

This is my current location in the terminal.

```
dell@dell-virdies:~$ 

```
Now, I want to go to `Downloads` folder where both of my files are located. Then we'll use this command.

```
cd Downloads
```
Note: Please don't make any typo mistakes.

Overall, it will look like this:

```
dell@dell-virdies:~$ cd Downloads
```

After executing this code, we'll be in the Downloads folder and now our command line will look like this:

```
dell@dell-virdies:~/Downloads $ 
```

Now as we are in the desired location, we'll decrypt the file using this command.
Please copy paste this code in your command line.

```
openssl enc -aes-256-cbc -d -salt -in test.txt -out output.txt -pass pass:simu123

```

Now, new '.txt' file will be created which will have the name as `output.txt`. Now as we want to see its content, we'll use this command.

```
cat output.txt
```


Now, you can see the decrypted message.