

do \<variable>=n,p,q
	block of code
end do
where n=value init, p is limit,q is step
loop start from n until p
so 1,2,3,..10

```
integer :: i

do i = 1, 10, 2
  print *, i  ! Print odd numbers
end do
```

do while (\<condition>)
	block of code
end do

```
integer :: i

i = 1
do while (i < 11)
  print *, i
  i = i + 1
end do
```

