> 使用laravel进行文件上传十分简单。以下贴出部分代码：

```php
public function upload(Request $request) {    
    if($request->isMethod('POST')){    
        //var_dump($_FILES);    
        $file = $request->file('source');    

        //判断文件是否上传成功    
        if($file->isValid()){    
            //获取原文件名    
            $originalName = $file->getClientOriginalName();    
            //扩展名    
            $ext = $file->getClientOriginalExtension();    
            //文件类型    
            $type = $file->getClientMimeType();    
            //临时绝对路径    
            $realPath = $file->getRealPath();    

            $filename = date('Y-m-d-H-i-S').'-'.uniqid().'-'.$ext;    
            $bool = Storage::disk('uploads')->put($filename, file_get_contents($realPath));    
            var_dump($bool);    
        }    

        //dd($file);    
        /** 
        *UploadedFile {#164 ▼ 
        *-test: false 
        *-originalName: "填充文件.png" 
        *-mimeType: "image/png" 
        *-size: 10340 
        *-error: 0 
        *path: "D:\xampp\tmp" 
        *filename: "phpF0E0.tmp" 
        *basename: "phpF0E0.tmp" 
        *pathname: "D:\xampp\tmp\phpF0E0.tmp" 
        *extension: "tmp" 
        *realPath: "D:\xampp\tmp\phpF0E0.tmp" 
        *aTime: 2016-11-22 04:39:27 
        *mTime: 2016-11-22 04:39:27 
        *cTime: 2016-11-22 04:39:27 
        *inode: 0 
        *size: 10340 
        *perms: 0100666 
        *owner: 0 
        *group: 0 
        *type: "file" 
        *writable: true 
        *readable: true 
        *executable: false 
        *file: true 
        *dir: false 
        *link: false 
        *linkTarget: "D:\xampp\tmp\phpF0E0.tmp" 
        *} 
        */    
        exit;    
    }    
    return view('student.upload');    
}
```
2333
