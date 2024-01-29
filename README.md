# mdk-functions

Project for exploring Azure Functions.

## How I created this project

Create a new Http Function project from template.

```bash
func init MdkFunctions --worker-runtime dotnet-isolated --target-framework net8.0
cd MdkFunctions
func new --name HttpExample --template "HTTP trigger" --authlevel "anonymous"
```

Personal preference: fix line endings to LF.

```bash
find . -type f | grep -v 'obj/' | grep -v 'bin/' | grep -v .git | while read f; do sed -i '' 's/\r//' $f; done
```


