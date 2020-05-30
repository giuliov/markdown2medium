# markdown2medium
Inspired by cjoudrey/md2medium, I want a simple way to re-publish in Medium some Markdown posts written for Hugo.

## Usage

```
markdown2medium                                                                                                     \
    --mediumIntegrationToken 1234567890abcdef1234567890abcdef123457890abcdef123456789abcdef1234                     \
    --markdownFile C:/myblog/content/post/2019/pyp/1-hosts/index.md                                                 \
    --canonicalURL http://blog.casavian.eu/2019/08/23/meta-pipelines-part-1-docker-hosts/                           \
    --publishStatus draft                                                                                           \
    --originalNote 'Originally posted at [{{ .BaseURL }}]({{ .CanonicalURL }}) on {{ .Date.Format \"2 Jan 2006\" }}'\
    --dryRun                                                                                                        \
    --debug
```