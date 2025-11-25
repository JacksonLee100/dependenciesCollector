# Dependencies Licenses & Version Collector

## Input

1. user will input path of folder like: "D:\Tst\dependenciesLicenes\tst"
2. user will input licenses.json file

## Output

Export all files's dependecies report of the input path, including the child folder

## Achieve Steps

1. make a filesname list of the  whole input path of folder, include child folder.
2. according to the dependencies name list of licenses.json file, scan the filesname list, if have the same name, save  dependency's name and its locations.
3. then scan *.h, *.cpp, *.csproj, pow.xml, package.json, package-lock.json, build.xml file content line by line, if match the key words from licenses.json dependenciesname, save dependency's name and its locations.
4. then collect step 2. and step 3. dependencies name with their locations, export them into dependencies_report.txt.

## Constrains
1. export dependencies_report.txt content should be like:
-lodash(1.0.0)[MIT]
 ├─D:\Tst\dependenciesScanner\package.json

2. there is open button to choose the input folder.

3. there is "licenses.json" button to import the licenses.json file

## Develop Env
Webapps


