# pipeutil

This is a pipeutil for golong to exec command !

## Usage:
```
cmds := []*exec.Cmd{
		exec.Command("ps", "-ef"),
		exec.Command("awk", "{print $2}"),
	}
	string, _ := pipeutil.ExecPipeLine(cmds)
	fmt.Printf(string)
```
