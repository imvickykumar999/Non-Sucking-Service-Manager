# NSSM Service Configurations

This document outlines the configurations for various services managed by NSSM (Non-Sucking Service Manager). Each section details the command used to edit the service, the application paths, and the input/output log file locations.

---

## Service: `bol7_dev_beat`

**Command:**
```

nssm edit bol7_dev_beat

```

**Application Details:**
* **Python Executable:** `D:\newbol7.com\env\Scripts\python.exe`
* **Working Directory:** `D:\newbol7.com\development`
* **Celery Command:** `D:\newbol7.com\env\Scripts\celery.exe -A bol7 beat --loglevel=info`

**I/O Logs:**
* **Output Log:** `D:\django_services\Logs\bol7_dev_beat_output.log`
* **Error Log:** `D:\django_services\Logs\bol7_dev_beat_error.log`

---

## Service: `bol7_dev_worker`

**Command:**
```

nssm edit bol7_dev_worker

```

**Application Details:**
* **Python Executable:** `D:\newbol7.com\env\Scripts\python.exe`
* **Working Directory:** `D:\newbol7.com\development`
* **Celery Command:** `D:\newbol7.com\env\Scripts\celery.exe -A bol7 worker --loglevel=info`

**I/O Logs:**
* **Output Log:** `D:\django_services\Logs\bol7_dev_worker_output.log`
* **Error Log:** `D:\django_services\Logs\bol7_dev_worker_error.log`

---

## Service: `chatbot_live_beat`

**Command:**
```

nssm edit chatbot_live_beat

```

**Application Details:**
* **Python Executable:** `D:\newbol7.com\chatbotbol7\env\Scripts\python.exe`
* **Working Directory:** `D:\newbol7.com\chatbotbol7\chatbot`
* **Celery Command:** `D:\newbol7.com\chatbotbol7\env\Scripts\celery.exe -A mychatbot beat --loglevel=info`

**I/O Logs:**
* **Output Log:** `D:\django_services\Logs\chatbot_live_beat_output.log`
* **Error Log:** `D:\django_services\Logs\chatbot_live_beat_error.log`

---

## Service: `chatbot_live_worker`

**Command:**
```

nssm edit chatbot_live_worker

```

**Application Details:**
* **Python Executable:** `D:\newbol7.com\chatbotbol7\env\Scripts\python.exe`
* **Working Directory:** `D:\newbol7.com\chatbotbol7\chatbot`
* **Celery Command:** `D:\newbol7.com\chatbotbol7\env\Scripts\celery.exe -A mychatbot worker --loglevel=info`

**I/O Logs:**
* **Output Log:** `D:\django_services\Logs\chatbot_live_worker_output.log`
* **Error Log:** `D:\django_services\Logs\chatbot_live_worker_error.log`
