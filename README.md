# swapOrgFolderGCP

Bash shell(swapOrgFolder.sh) will read all file in directory "inventory" and echo to csv format

## DataSource
| inventory/test01 | inventory/test02 |
|--------|--------|
| helloworld | helloworld_02 |
| 11111111111111 | 444444444444 |
| 22222222222222 | 555555555555 |
| 33333333333333 | 666666666666 |

## Result
| helloworld,33333333333333/22222222222222/11111111111111/ |
| ---------------------------------------------------------|
| helloworld_02,666666666666/555555555555/444444444444/ |
