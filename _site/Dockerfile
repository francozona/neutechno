# Use an official Jekyll image as the base
FROM jekyll/jekyll:latest

# Set the working directory inside the container
WORKDIR /srv/jekyll

# Copy the website files from your local machine to the container
COPY . .

# Install any Jekyll dependencies (if needed)
RUN bundle install

# Build the Jekyll website
RUN jekyll build

# Expose port 4000
EXPOSE 4000

# Command to start the Jekyll server
CMD ["jekyll", "serve", "--host", "0.0.0.0", "--port", "4000"]
