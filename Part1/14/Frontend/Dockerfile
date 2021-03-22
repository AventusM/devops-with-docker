FROM node
ENV REACT_APP_BACKEND_URL http://localhost:8080
EXPOSE 5000
COPY . .

# install serve
RUN npm install -g serve
# install dependencies
RUN npm install
# build static files
RUN npm run build

# run the application
CMD ["serve", "-s", "-l", "5000", "build"]