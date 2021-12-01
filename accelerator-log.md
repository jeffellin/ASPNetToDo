# Accelerator Log

## Options
```json
{
  "gitRepository" : "https://github.com/jeffellin/ASPNetToDo",
  "projectName" : "tanzu-dotnet-upgrade-accelerator",
  "repositoryPrefix" : "ellinj/cdemo"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**/*]
┃ ┃ ┃ ┃ ┃ Debug .tanzu/tanzu_tilt_extensions.py matched [**/*] -> included
┃ ┃ ┃ ┃ ┃ Debug .tanzu/wait.sh matched [**/*] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [**/*] -> included
┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [**/*] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**/*] -> included
┃ ┃ ┃ ┃ ┃ Debug k8s-resource.yaml matched [**/*] -> included
┃ ┃ ┃ ┃ ┗ Debug project.toml matched [**/*] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [k8s-resource.yaml, config/*.yaml, Tiltfile, README.md, catalog/*.yaml]
┃ ┃ ┃ ┃ ┃ Debug .tanzu/tanzu_tilt_extensions.py didn't match [k8s-resource.yaml, config/*.yaml, Tiltfile, README.md, catalog/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug .tanzu/wait.sh didn't match [k8s-resource.yaml, config/*.yaml, Tiltfile, README.md, catalog/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [k8s-resource.yaml, config/*.yaml, Tiltfile, README.md, catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [k8s-resource.yaml, config/*.yaml, Tiltfile, README.md, catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [k8s-resource.yaml, config/*.yaml, Tiltfile, README.md, catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug k8s-resource.yaml matched [k8s-resource.yaml, config/*.yaml, Tiltfile, README.md, catalog/*.yaml] -> excluded
┃ ┃ ┃ ┗ ┗ Debug project.toml didn't match [k8s-resource.yaml, config/*.yaml, Tiltfile, README.md, catalog/*.yaml] -> included
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [config/*.yaml, Tiltfile]
┃ ┃ ┃ ┃ ┃ Debug .tanzu/tanzu_tilt_extensions.py didn't match [config/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .tanzu/wait.sh didn't match [config/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [config/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/*.yaml, Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [config/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┗ Debug project.toml didn't match [config/*.yaml, Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [https://github.com->https://github.com/j...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [tanzu-dotnet->tanzu-dotnet-upgrade...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[2] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [your-registry.io/project->jeffellin/cdemo]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ Debug .tanzu/tanzu_tilt_extensions.py didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .tanzu/wait.sh didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┗ Debug project.toml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┗ ┗ ┗ ┗  Info Will replace [tanzu-dotnet->tanzu-dotnet-upgrade...(truncated)]
┃ ┗ ╺ engine.transformations[0].merge.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
