#找到网页源码中的第一个地址，已“<a href=”开始的地址

page= "....<a href="https.....">"

start_pos = page.find("<a href=")

start_quote = page.find('"', start_pos)

end_quote = page.find('"', start_quote+1)

url = page[start_quote+1, end_quote]


**********************************************************
#四舍五入

  function number_45(num)
  {
      num=num + 0.5;  (机智)
      num_str = str(num)
      position = num_str.find('.')
      print(num_str[:position])
  
  }
  
  **********************************************************
  #回文，正反读一样“madam”
  
  print(word.find(word[::-1]))
