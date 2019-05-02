# Routing

```javascript
this.router.navigateByUrl(`/courses/${course.id}`);

// Relative routing
constructor( private router: Router, private route: ActivatedRoute) {}

this.router.navigate(['courses', course.id])
this.router.navigate(['course.id'], { relativeTo: this.route });

// navigate with query params
this.router.navigate([`/courses`], { queryParams: {id: 37, username: 'jimmy'}});
```

```html
<a routerLink="courses" queryParams="{id: 37, username: 'jimmy'">GO</a>
```