



var words = [String]()

var line = readLine()
while line != nil && line != "" && line != " " {
    words.append(line!)
    line = readLine()
}

var pass = 0
var swapTotal = 0
var swap = 0

print("Pass: \(pass), Swaps: \(swap)/\(swapTotal), Array: \(words)")

for i in 1..<words.count {

    let currentNum = words[i]

    // all elements of array [0,i-1] that are greater than num to one position ahead of their current position

    var previousNum = i - 1 // index of previousNum
    var swap = 0
    while previousNum >= 0 && currentNum < words[previousNum] {
       
        words[previousNum+1] = words[previousNum] // previousNum takes place of currentNum
        previousNum -= 1
        swap += 1
        swapTotal += 1
    }
    words[previousNum+1] = currentNum
    pass += 1
    print("Pass: \(pass), Swaps: \(swap)/\(swapTotal), Array: \(words)")
    
   
}


