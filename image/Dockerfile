FROM public.ecr.aws/lambda/python:3.11

# copy the req.txt in the env variable of lambda
copy requirements.txt ${LAMBDA_TASK_ROOT}

RUN pip install -r requirements.txt

COPY src/* ${LAMBDA_TASK_ROOT}

CMD [ "main.handler" ]
