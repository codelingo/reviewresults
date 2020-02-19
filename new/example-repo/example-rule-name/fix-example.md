<!-- Use this as a template to outline an example of bad code vs fixed code -->

# Rule: Example Rule Name

## Fix Example

#### issue: filename.go:123
```diff
//Read file content by file path
func ReadAllFromFile(filePath string) ([]byte, error) {
	f, err := os.Open(filePath)
	if err != nil {
		return nil, err
	}
+	defer f.Close()

	return ioutil.ReadAll(f)
}
```

# Challenges to Scripting

## Custom Variables
...

## Subtle Logic
...

## Other
...
