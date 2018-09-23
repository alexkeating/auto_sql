# auto_sql

[![Build Status](https://travis-ci.org/brettvanderwerff/auto_sql.svg?branch=master)](https://travis-ci.org/brettvanderwerff/auto_sql)

==Work in progress== 

auto_sql is early in development,  more features to come

## Description

auto_sql is a memory aware csv to sqlite converter capable of converting multi-gigabyte tabular files to sqlite
databases on low memory machines. auto_sql focuses on speed by enabling multi-processing on multi-core machines.

## Installation

```commandline
$pip install auto_sql
```

## Usage Case

```python
import auto_sql

tab_obj = AutoSql(file='file.csv',
                        db_name='database',
                        sep='\t',
                        out_dir=".")

if __name__ == "__main__":
    tab_obj.run()

```

Currently auto_sql only supports csvs that contain headers

## Dependencies

* Python 3.4, 3.5, or 3.6

* pandas==0.21.1


* psutil==5.4.7
