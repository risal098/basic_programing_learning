
```
FUNCTION calculate_area(length, width) RESULT(area)
  REAL, INTENT(IN) :: length, width
  REAL :: area
  area = length * width
END FUNCTION

! Example usage
program main
  REAL :: l, w, a
  l = 5.0
  w = 10.0
  a = calculate_area(l, w)  ! Call the function and assign the result
  print *, "Area:", a
end program main
```