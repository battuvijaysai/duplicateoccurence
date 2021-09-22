my_str='jane is the best.Jane loves to cook.jane and will cook together'
print("the string is:")
print(my_str)
replace_dict={'Jane':'she'}
my_list=my_str.split('')
my_result=''.join([replace_dict.get(val) if val in replace_dict.keys() and my_list.index(val)!=idx else val for idx, val in enumerate(my_list)])
print("the string after replacing with value is:")
print(my_result)
