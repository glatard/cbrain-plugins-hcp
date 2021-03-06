# cbrain-plugins-hcp

CBRAIN plugins for pipelines of the Human Connectome Project. The
pipelines are installed in containers based on different versions of
the CentOS operating system.

* `PreFreeSurferPipelineBatch` is available in CentOS 5, 6 and 7. See
  containers on
  [DockerHub](https://hub.docker.com/r/bigdatalabteam/hcp-prefreesurfer/)
  (referred in the JSON descriptors).

*Important note to developers*: due to the handling of tool versions in the CBRAIN
Boutiques implementation, the tool interface will be shared by all the
versions of a given tool. Therefore, different versions of a tool must either:
* Share the same interface, i.e., inputs, output files, default values, etc.
* Be implemented as different tools, i.e., have different names.
