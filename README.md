#正则表达式

str='aabdfefkjkli'

aa=re.match('\D+','aabdfefkjkli')
bb=aa.group()
print(bb)

aa=re.search('\D+','aabdfefkjkli')
bb=aa.group()
print(bb)

