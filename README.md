# Test
Testing Purpose
func numberRightTringle(){
print("enter the no of row")
let n = Int(readLine()!)!
for i in 1..<n+1 {
    for j in 1...i {
        print(j, terminator: "")
    }
    print("")
}
 }
func sequecenrightTriangle(){
print("enter the no of row")
let n = Int(readLine()!)!
var value = 0
for i in 1...n {

    for _ in 1...i{
        value = value + 1
        print(value,terminator : "")
    }
    print(" ")
}
}
func pascalTrinagle(){
  print("enter the no of row:")
  let n = Int(readLine()!)!
        var no:Int = 1
        for i in 0...n{  
          for j in 0...i {
            if (j == 0 || i == 0){
                no = 1
            }else{
              no = no * (i - j + 1) / j
            }
            print("\(no)",  terminator: "")
          }
          print("")
        }
}
var tmp=1
repeat
{
  print("enter1.number right tringle pattern")
  print("enter2.for sequential number right tringle pattern")
  print("enter3.for pascal tringle pattern")
  print("enter0.for exit")
  print("enter your choice")
  let choice = readLine()
  switch choice! 
  {
    case "0":
          tmp=0
          print("quit..")
          break
    case "1":
        numberRightTringle()
    case "2":
        sequecenrightTriangle()
    case "3":
        pascalTrinagle()
    default:
        print("enter proper choice")
  }
}while(tmp != 0)
