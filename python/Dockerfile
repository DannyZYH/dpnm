ARG PYTHON_VERSION
FROM ${PYTHON_VERSION}

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /www

#pip配置为国内源
# RUN pip install tensorflow==1.14 -i https://pypi.tuna.tsinghua.edu.cn/simple
# RUN pip install opencv-python -i https://pypi.tuna.tsinghua.edu.cn/simple
# RUN pip install -r requirements -i https://pypi.tuna.tsinghua.edu.cn/simple [--timeout=60]
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install --upgrade pip

# COPY requirements.txt .
# RUN pip install -r requirements.txt
RUN pip install requires
RUN pip install pymysql
