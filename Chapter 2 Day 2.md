# Quest

## *1. Explain why we wouldn't call changeGreeting in a script*
* *Because changeGreeting is the name of the function which by calling it, it modifies data on the contract which is a transaction.*

## *2. What does the AuthAccount mean in the prepare phase of the transaction?*
* *The AuthAccount is used to access data in the account and it is done in the prepare phase of the transaction as the main purpose is to access information regarding the account.*

## *3. What is the difference between the prepare phase and the execute phase in the transaction?*
* *As mentioned earlier, the prepare phase's main purpose is to access data in the account. The execute phase calls for functions and is able to change data on the blockchain. Despite the fact that everything can be done in the prepare phase, it is better to separate logic and makes the code clearer.*

## *4.*
```
pub contract HelloWorld {

    pub var greeting: String
    
    pub var myNumber: Int 
    
    pub fun updatemyNumber(newNumber: Int) {
        self.myNumber = newNumber
    }
    pub fun changeGreeting(newGreeting: String) {
        self.greeting = "newGreeting"
    }
    init() {
        self.greeting = "Hello, World!"
        
        self.myNumber = 0
    }
}
```

![QuestSubmissions](https://github.com/DannyFlu/quest-submissions/blob/main/Quest%20C2D2.png)
