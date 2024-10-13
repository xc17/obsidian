### User Object Keys

```JSON
UserBoiler: {
	uid: string,
	name: string,
	dateCreated: Timestamp,
	email: string,
	nis: number,
	displayName: string,
	fullName: string,
	photoURL: string,
	class: string,

	// OPTIONS
	showPublicNIS: boolean,
	showPublicClass: boolean
}

UserExample: {
	uid: 'asdiu8gh978q2yhpsUsadi7wg',
	dateCreated: {
		...
	},
	email: 'email@address.com',
	nis: '12345',
	displayName: 'IfaaX',
	fullName: 'Ihsan Fashbir Danurrahardjo',
	photoURL: 'https://github.com/qwyzex/image',
	class: 'XI.6',

	// OPTIONS
	showPublicNIS: True,
	showPublicClass: False
}
```

