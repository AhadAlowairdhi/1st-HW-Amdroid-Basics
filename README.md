# 1st-HW-Android-Basics
## Print birthday cake - Tuwaiq Courses

### Ahad Alowairdhi

Description |

In this task, you are going to build a code to bake a cake to always be the right number of layers, size, and with the right number of candles.

Instructions |

You will create a total of three functions for drawing a layered cake with candles.
You will use a repeat() inside another repeat(), creating what's called a "nested loop".




##### The Solution:
[Run a program](https://pl.kotl.in/rafNxWTfK?theme=darcula) - kotlin playground
 ```
fun main() {
    val candles = 24
    val layers = 5
    println("Number of candels: $candles")
    println("Cake top length: $candles")
    println("Number of layers: $layers ")
    printCakeCandles(candles)
    printCakeTop(candles)
    printCakeBottom(candles,layers)
}

fun printCakeCandles(candles: Int){
    print(" ") // to be site a candles on the cake
    repeat(candles){
        print(",") 
    }
    println() // to print blank line
    
  	print(" ") // to be site a candles on the cake
    repeat(candles){
        print("|")
    }
    println() // to print blank line
}

fun printCakeTop(candles: Int){
    // +2 so that the candles won't to fall off the side of the cake 
   repeat(candles+2){
       print("=")
   }
   println() // to print blank line
}

fun printCakeBottom(candles: Int, layers: Int){
    //nested loop to print @ for 5 layers
   repeat(layers){
       repeat(candles+2){
       print("@")
   }
   println() // to print blank line
   }
    
}
```
