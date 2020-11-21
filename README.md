# Maximl-Labs
s = input()

window = set()
window.add(s[0])

i = 0; j = 1
ans = 1

while i<=j and j<len(s):
    if s[j] in window:
        window.remove(s[i])
        i+=1
    else:
        window.add(s[j])
        j+=1
    ans = max(len(window),ans)

print(ans)
