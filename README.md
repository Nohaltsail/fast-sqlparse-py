fast-sqlparse Library

Project Description:
fast-sqlparse is a SQL parsing library developed in C++ (C++17), designed for efficiently parsing large volumes of SQL statements, including long and complex queries. It supports parsing of SELECT, CREATE TABLE, INSERT, UPDATE, DELETE, and VIEW definition statements, as well as Common Table Expressions (CTEs). The library can also parse multiple SQL statements in a single input.

Core Features:
Lexical Analysis: Extract tokens from SQL statements.
Statement Structure Parsing: Obtain structured statement entities containing key components such as WHERE clauses, GROUP BY clauses, table aliases, etc.
Abstract Syntax Tree (AST) Generation: Build an AST representation of the parsed SQL.
SQL Formatting: Pretty-print or reformat SQL statements.
Comment Removal: Strip comments from SQL input.

Key Advantages:
Cross-platform: Currently supports both Linux and Windows environments.
High Performance: Operates in linear time complexity with low memory overhead.

Core Technologies:
A hand-written finite-state machine is used for lexical analysis, ensuring high performance.
During parsing, C++17’s string_view is leveraged to enable zero-copy syntax analysis, significantly reducing memory allocations and improving efficiency.
