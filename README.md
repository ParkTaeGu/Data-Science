# Data-Science
all about data science
def DFS(depth,index,sum):
    if(depth==3):
        if sum==0:
            rec.sort()
            temp=tuple(rec)
            if temp not in result:result.append(temp)      
        return

    if(index==len(S)):
        return

    rec.append(S[index])
    DFS(depth+1,index+1,sum+S[index]) 
    rec.remove(S[index]) 
    DFS(depth,index+1,sum)

DFS(0,0,0)
print(result)
