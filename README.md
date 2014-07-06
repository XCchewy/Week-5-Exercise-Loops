Week-5-Exercise-Loops
=====================

largest = None
smallest = None

while True:
    inp = raw_input('Enter a number: ')
    
    if inp == 'done' : break
    
    try:
        num = int(inp)
        
    except:
        print 'Invalid input'
        continue
    
    if largest is None or num > largest:
        largest = num
    if smallest is None or num < smallest:
        smallest = num
        
print 'Maximum is', largest
print 'Minimum is',smallest
