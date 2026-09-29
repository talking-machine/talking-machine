# Talking-Machine
A machine that talks.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Talk to me, machine." \
  | uvx talking-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install talking-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
talking-machine -a multilogue.txt
```
Or:
```bash
talking-machine multilogue.txt > response.txt
```
Or:
```bash
talking-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import talking_machine
```
