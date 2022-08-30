add_library(sqlparser
    parser/flex_lexer.cpp
    parser/bison_parser.cpp
    sql/Expr.cpp
    sql/CreateStatement.cpp
    sql/PrepareStatement.cpp
    sql/SQLStatement.cpp
    sql/statements.cpp
    util/sqlhelper.cpp
    SQLParserResult.cpp
    SQLParser.cpp
)

target_include_directories(sqlparser PUBLIC
 ../src
)

target_compile_features(sqlparser PUBLIC cxx_std_17)

target_compile_options(sqlparser PRIVATE "-Wall" "-Werror" "-Wno-sign-compare" "-Wno-unneeded-internal-declaration" "-O3")

