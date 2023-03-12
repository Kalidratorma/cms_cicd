FROM bellsoft/liberica-openjdk-alpine:17.0.6
# Set up the Environment Variable for Application
ENV APP_HOME=/app

# Create the directories for Application
RUN mkdir -p ${APP_HOME}

# Setting up the Work directory
WORKDIR ${APP_HOME}

ARG VERSION
ENV VERSION2=$VERSION
 
COPY ./core-$VERSION2.jar ${APP_HOME}

ENTRYPOINT java -jar core-${VERSION2}.jar
#CMD "java -jar ./core-$VERSION2.jar"
