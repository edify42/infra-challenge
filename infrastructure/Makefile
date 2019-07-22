# Makefile for the infrastructure as we don't need CI/CD for this example.

## variables
file := stack.yaml
stack_name := ed-kim-testing

## First make command is always the default :)
validate:
	aws cloudformation validate-template \
	--template-body file://${file}

create:
	aws cloudformation create-stack \
	--stack-name ${stack_name} \
	--template-body file://${file} \
	--capabilities CAPABILITY_IAM \
	--parameters "ParameterKey=param,ParameterValue=param-value"

destroy:
	aws cloudformation delete-stack --stack-name ${stack_name}

.PHONY: destroy