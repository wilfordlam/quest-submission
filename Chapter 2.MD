## Chapter 2 Day 1
Deploying the JacobTucker Contract

![image](https://user-images.githubusercontent.com/106781723/172920446-86e4bc41-0c01-4334-a98d-162daa607e67.png)

Checking the variable through execution of a script
![image](https://user-images.githubusercontent.com/106781723/172920542-793efaea-7c95-4364-8442-f69fb69b6856.png)

## Chapter 2 Day 2
1. When modifying a script, it does not modify the state of the contract. Here, we wanted to modify the state of our contract by changing our "greeting" field to be comething other than "Hello, World!". A script is used to view the results but cannot actually change anything about the transaction or the contract on the blockchain.
2. "AuthAccount" is type that allows the user to access the data in their account. As the user, you are authorizing the transaciton to take place in your account and access the data in your account.
3. "Prepare" is the phase where the transaction acesses the data in your account. Whereas, the "execute" phase calls the function to modiy the data on the blockchain. 
4. 
New Contract

![image](https://user-images.githubusercontent.com/106781723/172932717-ddca4620-6bb5-4e62-99ec-55af82f3c41b.png)

Transaction

![image](https://user-images.githubusercontent.com/106781723/172933217-2f580abc-4c19-4f28-8bab-a8d9299946ec.png)

Script

![image](https://user-images.githubusercontent.com/106781723/172933046-8ccec537-de69-4620-a3ad-e4c06adc019d.png)

## Chapter 2 Day 3
1. 3 names of Kobe, Hamilton, and Nadal were ran in a script

![image](https://user-images.githubusercontent.com/106781723/172954951-d50b21e5-2626-41f3-9120-1ce5bb9ed6b8.png)

2. Matching social media platform to usage

![image](https://user-images.githubusercontent.com/106781723/172955179-f4d7c2ee-33f8-4edc-97e9-b16efd72913f.png)

3. The foreced unwrap operator will obtain the value of an optional if it exsists
In the first instance below, the return value is an optional type without the forced unwrap at the end of the script. In the second image, the foreced unwrap was indicated so we are fore-unwrapping the optional

![image](https://user-images.githubusercontent.com/106781723/172957654-20b2c388-7fe6-44e7-a848-3f94d6e8283e.png)
![image](https://user-images.githubusercontent.com/106781723/172957702-7fde3322-6db5-43a2-b615-1cd333420eec.png)

4. The error indicates that there is a TYPE mismatch because it expected STRING but it got the optional STRING? This is beacuse the default setting is for an OPTIONAL type. This error can be amended via a fored-unwrap operator by putting "!" at the end of line 3. Now, there are no errors :)

## Chapter 2 Day 4
Combined 1-3

![image](https://user-images.githubusercontent.com/106781723/172963899-7467b228-b18c-4457-ad41-b73c5744ebb0.png)

Add a transaction to call that function in Step 3

![image](https://user-images.githubusercontent.com/106781723/172964001-cb85309d-143b-4e12-9568-80ca5c3a496e.png)

Add a script to read the Struct you defined

![image](https://user-images.githubusercontent.com/106781723/172964099-5929e14b-3692-4675-90bd-1582d67f271b.png)

## Chapter 3 Day 1
1. 3 reasons why structs are different form resoruces
- Resoruces cannot be copied 
- Resources cannot be overwritten
- You have to be explicit with Resources on how you use them/moving them. You cannot just leave them dangling at the end of the code

2. Resources are extremely useful for NFTs (makes sense since the FLOW ecosystem currently revovles mainly NFTs). This allows for easier tracking of digital ownership to see if NFTs are transferred or created

3. create

4. Transaction

5. Jacob

6. Erorrs:
- Jacob should be @Jacob
- Code should say let myJacob <- create Jacob()
- Missing the "move" operator "<-" after "return"
