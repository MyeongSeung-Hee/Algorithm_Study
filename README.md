# 2022-2 BaekJun Algorithm
## Algorithm_Study
### Week1
### Week2
### Week3
### Week4
#10828
import sys
N = int(sys.stdin.readline())

stack=[]
for _ in range(N):
    command = sys.stdin.readline().split()
    
    if(command[0] == "push"):
        stack.append(command[1])
        
    if(command[0] == "pop"):
        if(len(stack) == 0):
            print(-1)
        else:
            print(stack[-1])
            del(stack[-1])
    
    if(command[0] == "size"):
        print(len(stack))
        
    if(command[0] == "empty"):
        if(len(stack) == 0):
            print(1)
        else:
            print(0)
        
    if(command[0] == "top"):
        if(len(stack) == 0):
            print(-1)
        else:
            print(stack[-1])

#9093
import sys
 
n = int(sys.stdin.readline())
 
for _ in range(n):
  sentence = sys.stdin.readline().rstrip().split()
 
  for word in sentence:
    print(word[::-1], end=' ')
  print()

#1158
N, K = map(int, input().split(" "))

list = [j+1 for j in range(N)]

K -= 1
i = 0
ans = []

while len(list)!= 0:
    i = (i+K)%N
    ans.append(str(list[i]))
    del list[i]
    N -= 1

print("<",", ".join(ans)[:],">", sep='')
### Week5
### Week8
### Week9
### Week10
### Week11
### Week12
### Week13
