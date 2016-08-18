# hireable
Available-for-hire badge written in nodejs

## But why?
Some of my friends want to embed the employment status into their open-source projects.
But it takes too much time and effort to keep these information up-to-date across your projects.  
I thought it would be much cooler to tell people whether you're hireable or not with a badge. Isn't it? :confused:

## The badges
![Hireable](https://cdn.rawgit.com/hiendv/hireable/master/public/hireable-yes.svg)
![Not hireable](https://cdn.rawgit.com/hiendv/hireable/master/public/hireable-no.svg)
![Error](https://cdn.rawgit.com/hiendv/hireable/master/public/hireable-error.svg)

I was too lazy to implement [badges/shields specification](https://github.com/badges/shields/blob/master/spec/SPECIFICATION.md)  
No on-the-fly generated badges for now, I guess. They are all pre-generated. 

- Q: **How do you know when I'm hireable?**  
A: Your [GitHub jobs profile](https://github.com/settings/profile#user_profile_hireable)

- Q: **CDN?**  
A: Not sure if the badges need CDN. GitHub routes images through **camo** proxy. 

- Q: **Cache?**  
A: Should or shouldn't ? You tell me :thumbsup:

## Quickstart Installation
- Download the latest release [here](https://github.com/hiendv/hireable/releases)
```bash
# Unzip
unzip hireable-v*.zip -d hireable && cd hireable

# Dependencies
npm install --production

# Config
vim .env

# Serve
npm run serve

# Or even better with pm2 or forever
```

## Development
```bash
git clone https://github.com/hiendv/hireable.git && cd hireable
npm install
cp .env.example .env && vim .env
npm run dev

# Create a release?
npm run build && cd build
```

## Testing
```bash
npm test
```
e2e test PRs are welcome!
