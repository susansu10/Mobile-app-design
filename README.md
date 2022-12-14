# Mobile-app-design
2022/9 大四課
> 智慧行動應用與設計

## HW1 Kotlin-Programming 

### Solution :heavy_check_mark: 
```kotlin=
//Ex1
/*Student scores all are integers
*/
fun main() {
    var A_num = 0
    var B_num = 0
    var C_num = 0
    val scores = arrayOf(20, 40, 60, 80, 100)
    for (i in scores.indices) 
    {
        if(scores[i] >= 80 && scores[i] <= 100)
        {
            A_num += 1
        }
        else if(scores[i] >= 60 && scores[i] <= 79)
        {
            B_num += 1
        }
        else
        {
            C_num += 1
        }
    }
    println("A : $A_num")
    println("B : $B_num")
    println("C : $C_num")
}

//Ex2
fun factorial (n : Int) : Int
{
    var a = 1
    for(i in 2 until n + 1 )
    {
        a *= i
    }
    return a
}
/* My n terms is start from 1 ... n
 * Get_E(1) = 1
 * Get_E(2) = 1 + 1/1!
 * Get_E(3) = 1 + 1/1! + 1/2!
*/
fun Get_E(n : Int) : Double // 1 + 1/1! + 1/2!... + 1/n!
{
    var sum = 1.0
    for(i in 1 until n)
    {
        sum += 1.0 / factorial(i)
    }
    return sum
}

fun main() 
{
    var sum = Get_E(3)
    print(sum)
}

//Ex3
class rectangle(val length : Int, val width : Int)
{
    val area : Int
    	get() = width * length
    val perimeter : Int
    	get() = 2 *(width + length)
    fun info() = println("A rectangle with length = $length and width = $width")
    
}
fun main() 
{
    val recX = rectangle(10,20)
    println(recX.area)
    println(recX.perimeter)
    recX.info()
}
```

## HW2 Temperature Converter
![07](https://user-images.githubusercontent.com/75154678/200300762-138e7106-fc63-4109-83b6-42d8f8e93e2d.png)


## HW3 List of Sports
![HW3-01](https://user-images.githubusercontent.com/75154678/205625575-9be4cd43-a90a-49bc-8485-1a9aa0850c12.png)
![HW3-02](https://user-images.githubusercontent.com/75154678/205625663-4f7f8990-9ac7-430c-b9de-07b58861b367.png)



## Midterm-01 Simple Caculator 說明
![08](https://user-images.githubusercontent.com/75154678/200301914-a122da10-4959-4ed4-bd34-163ead3885f2.png)


## Midterm-02 DiceRoller 說明
![09](https://user-images.githubusercontent.com/75154678/200301963-38e2c7c8-69c5-45ff-bc63-e01fb82949ef.png)

