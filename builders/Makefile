BUILDERS_PREFIX := line/wasmvm-builder

.PHONY: docker-image-static
docker-image-static:
	docker build . -t $(BUILDERS_PREFIX):static -f ./Dockerfile.static

.PHONY: docker-images
docker-images: docker-image-static

# TODO publish images to registry
# .PHONY: docker-publish
# docker-publish: docker-images
# 	docker push $(BUILDERS_PREFIX):static
