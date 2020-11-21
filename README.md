# Maximl-Labs
s = input()

window = set()  
window.add(s[0])

i = 0; j = 1  
ans = 1

while i<=j and j<len(s):  
&nbsp;&nbsp;&nbsp;&nbsp;if s[j] in window:  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;window.remove(s[i])  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i+=1  
&nbsp;&nbsp;&nbsp;&nbsp;else:  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;window.add(s[j])  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;j+=1  
&nbsp;&nbsp;&nbsp;&nbsp;ans = max(len(window),ans) 

print(ans)
