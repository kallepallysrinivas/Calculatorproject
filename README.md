radius=5.0
perimeter=0.0
area=0.0
print"input the radius of the circle"
radius=gets.to_f
perimeter=2*3.14*radius
area=3.14*radius*radius
puts"The perimeter is #{perimeter}:"
puts"The area is #{area}:"

output:input the radius of the circle5.0
The perimeter is 31.400000000000002:
The area is 78.5:


2)puts"input your first name"
fname=gets.chomp
puts"input your last name"
lname=gets.chomp
puts "Hello #{lname} #{fname}"

ouput:ruby reverse.rb
input your first name
kallepally 
input your last name
srinivas
Hello srinivas kallepally 



3)puts"odd numbers between 9 to 1:"
9.step 1,-2 do|x|
puts "#{x}"
end


output:ruby oddnumbers.rb
odd numbers between 9 to 1:
9
7
5
3
1


4)def makes20(x,y)
return x==20||y==20|| x+y==20
end

print makes20(10,10),"\n"
print makes20(40,10),"\n"
print makes20(15,20) 



Output:ruby return20.rb
true
false
true

5)def temp(temp1,temp2)
return(temp1<0&&temp2>100)||(temp1>100&&temp2<0)
end
print temp(110,-1),"\n"
print temp(-1,110),"\n"
print temp(2,120)


output:ruby temp.rb
true
true
false


9)array1=["ruby",2.3,Time.now]
for array_element in array1
puts array_element
end


output:
ruby  printelements.rb
ruby
2.3
2025-04-04 12:25:55 +0530
