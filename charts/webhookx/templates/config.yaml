{{- if .Values.config.enabled }}
apiVersion: v1
kind: ConfigMap
metadata:
  name: {{ include "webhookx.fullname" . }}-config
  labels:
    app.kubernetes.io/name: {{ include "webhookx.name" . }}
    app.kubernetes.io/instance: {{ .Release.Name }}
    app.kubernetes.io/component: config
data:
{{- range .Values.config.data }}
  {{ .name }}: "{{ .value }}"
{{- end }}
{{- end }}