#找到网页源码中的第一个地址，已“<a href=”开始的地址

page= "....<a href="https.....">"

start_pos = page.find("<a href=")

start_quote = page.find('"', start_pos)

end_quote = page.find('"', start_quote+1)

url = page[start_quote+1, end_quote]


  _______________________________________________________
#四舍五入

  function number_45(num)
  {
      num=num + 0.5;  (机智)
      num_str = str(num)
      position = num_str.find('.')
      print(num_str[:position])
  
  }
    _______________________________________________________
    
  #回文，正反读一样“madam”
  
  print(word.find(word[::-1]))
  
  _______________________________________________________
  # Define a procedure, median, that takes three
# numbers as its inputs, and returns the median
# of the three numbers.

# Make sure your procedure has a return statement.

def bigger(a,b):
    if a > b:
        return a
    else:
        return b

def biggest(a,b,c):
    return bigger(a,bigger(b,c))

def median(a, b ,c):
    big=biggest(a,b,c)
    if a== big:
      return bigger(b,c)
    if b== big:
      return bigger(a,c)
    if c== big:
      return bigger(b,a)
      
  _______________________________________________________
  #给出三个数的范围
  
  def bigger(a,b):
    if a >b:
        return a
    else 
        return b
        
def biggest(a,b,c):
    return bigger(a, bigger(b,c))
    
def set_range(a,b,c):
    # Your code here
    n = biggest(a,b,c)
    return biggest(n-a, n-b, n-c)
