# byd
# 做简单的循环语句插入练习
file = open(r"D:\aabb.txt", "w")

for i in range(1, 1000):
    file.write("INSERT INTO  `tag_table` "
               "( `pk_v_i`, `tag_i`, `name`, `display_name`, `lang_code`, `category_i`, `update_date`, `seq`, `ext_val1`, `ext_val2`, `ext_val3` )" +
               " VALUES ( " +
               str(i) + ", " +
               "270" +", "+
               ("`BS_15_Others" + "{:0>2d}".format(i) + "`," +
               "`Others`"+","+
               "`cn` ,"+"20 ,"+"`2021-02-08 14:02:19` ,"+
                "`North America" + "{:0>2d}".format(i) + "`)" '\n'))

file.close()





