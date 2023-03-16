# Kotlin-Example


Practical 1.1.1
Aim:- Dog hears frequencies starting from 67 Hertz to 45000 Hertz (both
inclusive).
Pass value X Hertz, ﬁnd whether dog can hear them or not.
Print YES if value between 67 to 45000. Otherwise print NO

Code in Kotlin:
fun main() {
// create scanner object to take input from user
val scanner = Scanner(System.`in`)
// take input from user
print("Enter the frequency value in Hertz: ")
val frequency = scanner.nextInt()
// check if frequency is within dog's hearing range
if (67 <= frequency && frequency <= 45000) {
println("YES, the dog can hear this frequency.")
} else {
println("NO, the dog cannot hear this frequency.")
}
// close scanner object
scanner.close()
}

Practical 1.1.2
Aim:- Let's assume there is one fest name VIBES and you want to visit with
your friend. You manage to collect passes for fest.
A person can enter the fest using one pass, and each pass can be used by
only one person.
Take two input one no. of passes you have and Second no. of you
are.
Print YES if all person enter in the fest with available passes
otherwise print NO.
Note:- In Second Input You are excluded.

Code in Kotlin:
import java.util.Scanner
fun main() {
// create scanner object to take input from user
val scanner = Scanner(System.`in`)
// take input from user
print("Enter the number of passes you have: ")
val numPasses = scanner.nextInt()
print("Enter the number of friends you have (excluding yourself): ")
val numFriends = scanner.nextInt()
// check if all friends can enter the fest with available passes
if (numPasses >= numFriends) {
println("YES, all friends can enter the fest with available passes.")
} else {
println("NO, all friends cannot enter the fest with available passes.")
}
// close scanner object
scanner.close()
}


Practical 1.1.3
Aim:- A participant can make 1 submission every 30 seconds. If a contest
lasts for X minutes, what is the maximum number of submissions that the
participant can make during it?

fun main() {
    val minutes = 60 // set the contest duration in minutes
    val submissionsPerMinute = 2 // participant can make 2 submissions per minute
    val maxSubmissions = submissionsPerMinute * minutes
    println("Maximum submissions: $maxSubmissions")
}



Practical 1.1.4
Aim:- A lamp is Off and can be on print if the lamp is on or off

import java.util.*

fun main() {
    println("Lamp is ON or OFF?")
    val sc = Scanner(System.`in`)
             val isStatus = sc.nextLine()
    if(isStatus == "ON" || isStatus == "on") {
        println("Lamp is ON")
    } else if(isStatus.lowercase() == "off") {
        println("Lamp is OFF")
    } else {
        println("Invalid Status")
    }
}
