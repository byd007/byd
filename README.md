# byd

file = open(r"D:\aabb.txt", "w")

for i in range(1, 1000):
    file.write("INSERT INTO  `tbl_metadata_tag_value_definition` "
               "( `pk_value_id`, `tag_id`, `name`, `display_name`, `lang_code`, `category_id`, `update_date`, `seq`, `ext_value1`, `ext_value2`, `ext_value3` )" +
               " VALUES ( " +
               str(i) + ", " +
               "270" +", "+
               ("`BS_15_Others" + "{:0>2d}".format(i) + "`," +
               "`Others`"+","+
               "`cn` ,"+"20 ,"+"`2021-02-08 14:02:19` ,"+
                "`North America" + "{:0>2d}".format(i) + "`)" '\n'))

file.close()





