query {
  postCollection(limit: 3) {
    items {
      title,
      slug,
      excerpt,
      date,
      coverImageUrl,
      authorName {
        sys {
          id
        }
      },
      pictureUrl
    }
  }
  
  authorCollection {
    items {
      name
      pictureUrl,
      title,
      linkedPostsTitlesCollection {
        items {
          sys {
            id
          }
        }
      }
    }
  }
  
  post(id: "43MeN2SUXbAaSwjFyEp9g2") {
    title
  }
}